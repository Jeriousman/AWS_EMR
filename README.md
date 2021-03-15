# AWS_EMR

This is how to install and use AWS EMR
https://youtu.be/fC4Y7KNwRzs 
https://www.youtube.com/watch?v=qv1ErFMmhC4



# EMR 클러스터 생성

클러스터생성은 원하는 EC2 타입을 정하고 키페어를 설정하고 생성한다. EC2 R과 M 타입 & 5.1x 이하 버전에서는 EMR Notebook을 사용할 수 없으니 참고하여 생성한다.
클러스터가 시작에서 대기가 되면 클러스터가 제대로 작동할 준비를 마친 것이니 사용해도 된다.



# EMR 연결

EMR의 마스터노드에 들어가 EC2위에 커서를 대고 연결 (Connect)를 누른다. 거기서 알려주는 주소 [예) ssh -i "aws_password.pem" ec2-user@ec2-3-141-8-15.us-east-2.compute.amazonaws.com]
를 AWS CLI (커맨드라인)에서 키페어.pem 파일이 있는 곳으로 경로 이동을 한 후 입력한다. 


# PySpark 연결

EMR에 연결되었을 때 AWS CLI 콘솔에 pyspark을 치면 PySpark에 접속된다. 이로써 파이썬코드로 Spark을 사용 할 수 있다.
