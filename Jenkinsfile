pipeline {
agent any

stages {
stage ('build') {
steps {
sh '''
echo "creating build files"
   dd if=/dev/zero of=bigfile bs=1G count=22
echo "created build files"
'''
}
}
}
}


