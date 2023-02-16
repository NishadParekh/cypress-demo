node {
  stage ('checkout code from git hub') {
    git branch: 'main', url: 'https://github.com/NishadParekh/cypress-demo.git'
  }
  stage ('install node js') {
    sh "apt update" 
    sh "apt install nodejs -y"
    sh "apt install npm -y"
    sh "npm init -y"
   }
  stage('intall cypress') {
    sh "npm install --save -dev cypress"
    sh "apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb -y"
    sh "npx cypress run"
    
  }
}
