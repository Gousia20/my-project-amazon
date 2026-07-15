pipeline {
agent any

stages {
stage ('build') {
steps {
sh '''
echo "creating build files"
rm -rf bigfile
mkdir -p bigfile
   dd if=/dev/zero of=bigfile/testfile.img bs=1G count=30
echo "created build files"
df -h /
exit 1
'''
}
}
}
post {
    always {
        sh 'rm -rf bigfile'
    }
}
}


