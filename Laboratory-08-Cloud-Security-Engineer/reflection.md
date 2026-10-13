# Mission Reflection

This laboratory helped me understand how a host-based firewall protects a server by controlling the network connections it accepts. Even when a system is connected to a larger network, firewall rules can provide an additional layer of defense by limiting access to approved services.

I learned that open ports should be managed carefully because each accessible service may introduce a potential security risk. During the activity, I practiced allowing SSH for remote administration and TCP port 8080 for the Nginx application while applying a default policy that rejects incoming connections unless they are permitted.

The activity also helped me understand the risks of exposing database services, such as MySQL on port 3306, to the public internet. Public access can increase the likelihood of unauthorized connection attempts. Database services should instead be restricted to trusted systems and authorized users whenever possible.

Another lesson was the importance of checking firewall rules after making changes. A firewall must allow the connections needed by the application while restricting unnecessary traffic. When managing a server remotely, the SSH rule should be configured before enabling UFW to avoid losing administrative access.

After completing the laboratory missions, I have developed a better understanding of different cloud computing responsibilities, including deployment, operations, and security. These activities have shown me how proper configuration and verification contribute to a more reliable environment.

Overall, this mission taught me that server security requires careful planning and regular review. Applying suitable firewall rules, testing required services, and limiting unnecessary access are important practices for maintaining a secure system.
