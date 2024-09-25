
terraform/.gitignore - позволить временным и служебным файлам не попасть в git репозиторий, игнорируруемые файлы большого размера и каждый раз при выполнение кода террафом будут созданы заново. Хранить их в каком либо репозитории не имеет смысла! Также это могут быть файлы-ключи содержащие какую ту информацию включая токены которые не должны попасть в открытое пространство!



**/.terraform/*
- будут игнорироваться файлы,  в папке /.terraform/ . сама папка /.terraform/ может быть в любом месте проекта, т.е. у нее любая вложенность
 

*.tfstate 
- будут игнорироваться файлы с расширением *.tfstate

*.tfstate.*
- будут игнорироваться файлы содержащие  в имени tfstate


crash.log
- игнорируем crash.log файл  

crash.*.log
- игнорируем файлы начинающиеся на "crash." с расширением "log"

*.tfvars
*.tfvars.json
- игнириуеться файлы с расширением "tfvars" и "tfvars.json"


 
override.tf
override.tf.json
- игнорируем файлы "override.tf" и "override.tf.json"

*_override.tf
*_override.tf.json
- игнорируем файлы чьи имена оканчивающиеся на "_override.tf" и "override.tf.json"


.terraform.tfstate.lock.info
- игнорируем файл ".terraform.tfstate.lock.info"

 
.terraformrc
terraform.rc
- игнорируем файл ".terraformrc" и "terraform.rc"