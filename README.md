# ubuntu-server-odoo-service-down   
[Service]   
Type=simple   
User=odoo   
ExecStart=/opt/odoo/odoo-bin -c /etc/odoo/odoo.conf   
# addthis to your service   
Restart=always   
RestartSec=5   
# after that    
sudo systemctl daemon-reload   
sudo systemctl enable odoo   
sudo systemctl restart odoo   
