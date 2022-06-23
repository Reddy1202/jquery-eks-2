aws ecr get-login-password --region ap-south-1 | sudo docker login --username AWS --password-stdin 897025645367.dkr.ecr.ap-south-1.amazonaws.com


sudo docker build -t jquery-eks2:latest 897025645367.dkr.ecr.ap-south-1.amazonaws.com/jquery-eks2:$BUILD_NUMBER .

sudo docker push 897025645367.dkr.ecr.ap-south-1.amazonaws.com/jquery-eks2:$BUILD_NUMBER