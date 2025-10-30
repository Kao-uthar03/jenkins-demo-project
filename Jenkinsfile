// Jenkinsfile
@Library('ma-lib-partagee') _

pipeline {
    agent any

    stages {
        stage('Utiliser MonUtilitaire') {
            steps {
                script {
                    org.exemple.utils.MonUtilitaire.saluer(this, "Jenkins User")
                    def messageSucces = org.exemple.utils.MonUtilitaire.genererMessage("succes")
                    echo messageSucces
                }
            }
        }

        stage('Utiliser autreFonction') {
            steps {
                script {
                    def resultat = autreFonction("Ceci est un test de fonction globale.")
                    echo "Résultat de autreFonction : ${resultat}"
                }
            }
        }
    }
}
