node {
  stage ('checkout code from git hub') {
    git branch: 'main', url: 'https://github.com/NishadParekh/cypress-demo.git'
  }
  stage ('install node js') {
    sh "apt install nodejs"
    sh "npm init"
   }
  stage('intall cypress') {
    sh "npm install --save -dev cypress"
    sh "npx cypress open"
    
  }
}
