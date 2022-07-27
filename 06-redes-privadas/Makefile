
delete-staging:
	aws cloudformation delete-stack --stack-name staging-vpc || exit 0
deploy-staging:
	aws cloudformation deploy --stack-name staging-vpc --template-file stack-vpc.yaml --parameter-overrides Environment=staging VPCCidrBlock=192.168.0.0/16 PublicSubnectCidrBlocks="192.168.10.0/24,192.168.20.0/24,192.168.30.0/24" PrivateSubnectCidrBlocks="192.168.110.0/24,192.168.120.0/24,192.168.130.0/24"


delete-prod:
	aws cloudformation delete-stack --stack-name prod-vpc || exit 0
deploy-prod:
	aws cloudformation deploy --stack-name prod-vpc --template-file stack-vpc.yaml --parameter-overrides Environment=production VPCCidrBlock=192.168.0.0/16 VPCCidrBlock=192.168.0.0/16 PublicSubnectCidrBlocks="192.168.10.0/24,192.168.20.0/24,192.168.30.0/24" PrivateSubnectCidrBlocks="192.168.110.0/24,192.168.120.0/24,192.168.130.0/24"

