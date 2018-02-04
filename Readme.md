#add mysql support as below

pip install PyMySQL

GRANT ALL PRIVILEGES ON foxjar.* TO 'ujar'@'localhost' IDENTIFIED BY 'shadowfox';
GRANT ALL PRIVILEGES ON foxdjg.* TO 'udjg'@'localhost' IDENTIFIED BY 'shadowfox';
python manage.py shell
from django.contrib.auth.models import User  
user=User.objects.create_superuser('fox','cuiyingjia@foxmail.com','shadowfox')  
