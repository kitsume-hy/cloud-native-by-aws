# Chapter4 memo
- aws ec2 create-key-pair コマンドでKeyMaterialをダブルクォートで囲む.

` aws ec2 create-key-pair --key-name {key_name} --query "KeyMaterial" --output text > {key_name}pem `

