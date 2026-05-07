# What is this?
This is a multi-threading transformation of Odoo 16's multi-process mode, enabling each worker to launch multiple threads to handle user requests. For I/O-intensive applications, this effectively reduces memory consumption and improves concurrency.

# How to deploy?
copy src/server.py to odoo/service/server.py
then restart odoo

# How to set worker thread per process?
add the following line to odoo.conf
workers_threads = 6
