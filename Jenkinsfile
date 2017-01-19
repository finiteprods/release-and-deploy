node {
   stage('Preparation') {
      git 'https://github.com/finiteprods/release-and-deploy.git'
   }
   stage('Build') {
      bat "./gradlew clean test"
   }
   stage('Deploy') {
      bat "git push https://git.heroku.com/afternoon-bayou-45856.git master"
   }
}