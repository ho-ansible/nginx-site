# Ansible role: nginx-site
Populate content for a site from a git repo

# Dependencies
+ nginx

# Role Variables
+ `site_repo`: git URL to content
+ `site_branch` (default: master): which branch to pull from git
+ `site_name`: short identifier
+ `site_config` (default: `{{ inventory_dir }}/.sites/{{ site_name }}`):
  nginx config file
+ `site_dir` (default: `/var/www/{{ site_name }}`): where to store site content
+ `site_ports` (default: [443]): ports to open up on firewall
