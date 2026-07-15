pipeline {
agent any

stages {
stage ('build') {
steps {
sh '''
echo "creating build files"
mkdir -p bigfile
   dd if=/dev/zero of=bigfile/testfile.img bs=1M count=500
echo "created build files"
'''
}
}
}
}


