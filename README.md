Beancount configuration to read ofx/qfx with smart importer

Usage:
sudo docker run -v $(pwd):/data beancount bean-check example.beancount
sudo docker run -v $(pwd):/data beancount bean-extract example.import /data/ofxdownload.ofx -e example.beancount
sudo docker run -v $(pwd):/data beancount [bean-command]
