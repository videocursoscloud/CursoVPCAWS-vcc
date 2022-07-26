
delete-staging:
	aws cloudformation delete-stack --stack-name staging-vpc 
deploy-staging:
	aws cloudformation deploy --stack-name staging-vpc --template-file stack-vpc.yaml --parameter-overrides Environment=staging 


delete-prod:
	aws cloudformation delete-stack --stack-name prod-vpc 
deploy-prod:
	aws cloudformation deploy --stack-name prod-vpc --template-file stack-vpc.yaml --parameter-overrides Environment=production

