pipeline {
 agent any
 stages {
 stage('confirm version') {
 steps {
 nodejs('Node18.4.0') {
 sh 'node -v'
 sh 'npm -v'
 }
 }
 }
 stage('install node packages') {
 steps {
 nodejs('Node18.4.0') { // <- use node name you configured 
 in “Global Tool Config”.
 sh 'npm install'
 }
 }
 }
 }
}
