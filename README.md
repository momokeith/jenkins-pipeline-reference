 curl -Lv http://ec2-176-34-135-67.eu-west-1.compute.amazonaws.com/login 2>&1 | grep 'X-SSH-Endpoint'
 ssh -l mkeita -p 56685 ec2-176-34-135-67.eu-west-1.compute.amazonaws.com help
 add SSH KEY to jenkins
 https://JENKINS_URL/jnlpJars/jenkins-cli.jar
 scp Jenkinsfile devops:/tmp && ssh devops "ssh -l mkeita -p 56685 ec2-176-34-135-67.eu-west-1.compute.amazonaws.com declarative-linter < /tmp/Jenkinsfile"