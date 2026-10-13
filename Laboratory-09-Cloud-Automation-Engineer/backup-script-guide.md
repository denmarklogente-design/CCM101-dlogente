# Backup Script Guide

## 1. Purpose

The backup script creates a compressed archive of the `app-data` directory and saves it in the `backups` folder. A timestamp is included in the filename to distinguish backups created at different times.

## 2. Full Bash Script

```bash
#!/bin/bash
# Backup Automation for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Starting the backup process..."

# Create the destination folder if needed
mkdir -p "$BACKUP_DIR"

# Create a compressed archive
if tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"; then
    echo "Backup completed successfully at $TIMESTAMP!"
else
    echo "Backup failed. Please check the source directory and permissions."
    exit 1
fi
```

## 3. File Permissions

The command below grants executable permission to the script:

```bash
chmod +x backup.sh
```

After setting the permission, run the script using:

```bash
./backup.sh
```

The command must be executed from the appropriate directory, and the user must have permission to access the required files and folders.

## 4. Cron Schedule

The following Cron entry schedules the backup script to run daily at 2:00 AM:

```cron
0 2 * * * /root/backup.sh
```

The five fields in the schedule represent the following:

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The path `/root/backup.sh` must match the actual location of the script. The schedule follows the system's configured time zone.

## 5. Verification

Use the following command to list the generated backup archives:

```bash
ls -lh backups/
```

To inspect an archive, run:

```bash
tar -tzf backups/backup_FILENAME.tar.gz
```

Replace `backup_FILENAME.tar.gz` with the actual archive filename. If the command lists the archived files without an error, the archive can be read and its contents inspected.
