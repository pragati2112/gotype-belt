# login into ECR
```
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 522354467085.dkr.ecr.us-east-1.amazonaws.com
```

# build pulseapi
```
docker build -t 522354467085.dkr.ecr.us-east-1.amazonaws.com/pulseapi .
```

# push to ecr
```
docker push 522354467085.dkr.ecr.us-east-1.amazonaws.com/pulseapi:latest
```



# build pulseapi
```
docker build -t 522354467085.dkr.ecr.us-east-1.amazonaws.com/pulseweb .
```

# push to ecr
```
docker push 522354467085.dkr.ecr.us-east-1.amazonaws.com/pulseweb
```
