# Supervisor
A collection of scripts to manage a Supervisor instance on a remote VPS (virtual private server) on Linode.

[Supervisor](http://supervisord.org/introduction.html) is a client/server system for managing multiple processes on a single UNIX environment under one system.

In my workflow, I manage multiple python apps that are all self contained in their own virtual environment (venv). Supervisor allows you to start processes in their own environments.

### Getting Started
1. Create and start a Python Virtual Environment `python3 -m venv venv` `. venv/bin/activate`
2. Install Supervisor using `pip install supervisor`. `requirements.txt` is for version tracking `pip install -r requirements.txt`.
3. Launch Supervisor with `venv/bin/supervisord -c supervisord.conf`
4. Manage Supervisor using `venv/bin/supervisorctl`

- It maybe possible to launch Supervisor without `venv`

### Next Steps
- Running Supervisor on startup (systemd/linux service)



*Author: Duc Cong Duong*
