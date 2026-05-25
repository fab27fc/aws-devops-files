## Update y crear carpeta
sudo yum -y update
##
mkdir ~/efs-mount-point 

# Instalar utilidades de EFS
sudo yum install -y amazon-efs-utils

# Montar utilizando el Mount Helper
sudo mount -t efs <fs-0b051c875579db2d2>:/ ~/efs-mount-point

# Desmontar el sistema de archivos EFS
sudo umount ~/efs-mount-point

# Verificar
df -h
