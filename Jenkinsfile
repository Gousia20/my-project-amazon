pipeline {
agent any

stages {
stage ('build') {
steps {
sh '''
echo "disk space before"

df -h
   dd if=/dev/zero of=bigfile bs=1G count=22
echo "disk space after"
'''
}
}
}
}.


