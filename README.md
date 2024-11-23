# NT548-lab2-group9-CloudFormation-CodePipeline
NT548-lab2-group9-CloudFormation-CodePipeline

Members of group 9:
| MSSV | FullName | Email |
|-------------|-----------------------|---------------------------------|
| 21521023| Nguyễn Đức Trung Kiên | 21521023@gm.uit.edu.vn |
| 21522530 | Hoàng Tất Quý | 21522530@gm.uit.edu.vn |
| 21522604 | Phùng Nam Thanh | 21522604@gm.uit.edu.vn |
| 21522729 | Đỗ Xuân Trường | 21522729@gm.uit.edu.vn |

STEP:
- git clone
- aws configure
- make Github Token and save it in Secret AWS 
- make s3 bucket with cloudformation-modules name
- aws s3 cp [Name of modules].yml s3://cloudformation-modules
- aws cloudformation delete-stack --stack-name [Name of Stack]
- aws cloudformation create-stack --template-body file://[URL to the sample file in your PC] --stack-name [Name of Stack] --capabilities CAPABILITY_NAMED_IAM --parameter-overrides GitHubOwner=[GitHub Username]