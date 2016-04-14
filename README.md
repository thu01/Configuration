# Configuration
## VIM Configuration
1. Install Vundle 
2. Install other plugins with Vundle

## Apache + PHP Configuration

####  Run Apache  
```
apachectl start
``` 

#### Enable PHP for Apache
```
# Make backup for configuration file
cd /etc/apache2/    
cp httpd.conf httpd.conf.bak  
```  
```
# Edit Apache configuration
vi httpd.conf
```       
```
# Enable php module, uncomment the following line
LoadModule php5_module libexec/apache2/libphp5.so   
```    
```
# Restart Apache
apachectl restart  
``` 

#### More configuration settings   
```
# Support more index files
DirectoryIndex index.php index.html  
```   
```
# Set document root
DocumentRoot "/Users/yourusername/Sites/"  
<Directory "/Users/yourusername/Sites/">  
```  
    
