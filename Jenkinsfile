// Declarative //
pipeline {
agent any
stages {
stage('Test') {
steps {
/* `make check` returns non-zero on test failures,
* using `true` to allow the Pipeline to continue nonetheless
*/
sh '''  
pwd
cd $HOME
pwd
sh 'make'
junit '**/target/*.xml'
'''
}
}
}
}
