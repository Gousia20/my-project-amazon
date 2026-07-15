pipeline {
agent any

stages {
stage ('build') {
steps {
sh '''
echo "creating build files"
mkdir -p bigfile
   dd if=/dev/zero of=bigfile bs=1G count=22
echo "created build files"
'''
}
}
}
}


