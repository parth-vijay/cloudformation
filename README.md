# cloudformation

    aws cloudformation create-stack --stack-name ec2-example --template-body file://01_ec2.yaml      (Create CloudFormation stack)
    aws cloudformation delete-stack --stack-name ec2-example                                         (Delete CloudFormation stack)

    aws cloudformation update-stack --stack-name ec2-example --template-body file://04_ec2.yaml --parameters ParameterKey=AvailabilityZone ParameterValue=ap-south-1 ParameterKey=EnvironmentType,ParameterValue=dev ParameterKey=KeyPairName,ParameterValue=cloudformation

    aws cloudformation create-stack --stack-name rds-example --template-body file://05_rds.yaml --parameters ParameterKey=AvailabilityZone,ParameterValue=ap-south-1a ParameterKey=EnvironmentType,ParameterValue=dev ParameterKey=KeyPairName,ParameterValue=cloudformation ParameterKey=DBPassword,ParameterValue=Abcd1234