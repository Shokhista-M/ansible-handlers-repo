# ansible-handlers-repo
Create an Ansible playbook that does the following on a CentOS system:

Installs the httpd package.

Deploys a website configuration file using an Ansible template (.j2 file) to /etc/httpd/conf.d/mywebsite.conf.

The template should include:

A line with ServerName {{ ansible_hostname }}

A line with DocumentRoot /var/www/html/mywebsite

If the template changes, use a handler to restart the httpd service.

Ensure that the /var/www/html/mywebsite directory exists.

Create an index.html file inside that directory with the text:

Welcome to my Ansible-powered website!


Make sure the httpd service is enabled and running.

Print a debug message:
"Website deployed successfully on {{ ansible_hostname }}"