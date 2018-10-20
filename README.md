## Beancount configuration to read ofx/qfx with smart importer

### Example:
example.beancount: existing beancount file  
example.import: configuration for ofx account  
ofxdownload.ofx: downloaded statement in ofx/qfx format  

sudo docker run -v $(pwd):/data beancount bean-check example.beancount  
sudo docker run -v $(pwd):/data beancount bean-extract example.import /data/ofxdownload.ofx -e example.beancount  

The accounts are automatically added by [smart-importer](https://github.com/beancount/smart_importer)  
Notice the accounts are added incorrectly for transactions not present in example.beancount  

Any other bean command can be excecuted:  
sudo docker run -v $(pwd):/data beancount [bean-command]
