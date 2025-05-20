# ubuntu-server-odoo-service-down   
[Service]   
Type=simple   
User=odoo   
ExecStart=/opt/odoo/odoo-bin -c /etc/odoo/odoo.conf   
Restart=always  # addthis to your service   
RestartSec=5   # addthis to your service   
after that    
sudo systemctl daemon-reload   
sudo systemctl enable odoo   
sudo systemctl restart odoo   
