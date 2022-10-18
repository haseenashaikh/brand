pipeline{
    agent any
    stages{
        stage('git clone'){
            steps{
                sh'''
                pwd
                rm -rf *
               git clone https://github.com/haseenashaikh/brand.git
                '''
            }
        }
        stage('maven1'){
            steps{
                sh'''
                cd brand
                mvn clean
                '''
            }
        }
        stage('maven2'){
            steps{
                sh'''
                cd brand
                mvn test
                '''
            }
        }
        stage('maven3'){
            steps{
                sh'''
                cd brand
                mvn clean
                '''
            }
        }
        stage('maven4'){
            steps{
                sh'''
                cd brand
                mvn install package
                '''
            }
        }
    }
}
