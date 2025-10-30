// Jenkinsfile
@Library('ma-lib-partagee') _

pipeline {
    agent any

    stages {
        stage('Utiliser MonUtilitaire') {
            steps {
                script { // Ce bloc script est déjà présent, c'est bien.
                    org.exemple.utils.MonUtilitaire.saluer(this, "Jenkins User")
                    def messageSucces = org.exemple.utils.MonUtilitaire.genererMessage("succes")
                    echo messageSucces
                }
            }   
        }
    }
}

        stage('Utiliser autreFonction') {
            steps {
                // 'def resultat = ...' est une déclaration de variable Groovy,
                // et l'appel de 'autreFonction' est une étape que l'on veut capturer dans une variable.
                script {
                    def resultat = autreFonction("Ceci est un test de fonction globale.")
                    echo "Résultat de autreFonction : ${resultat}"
                    }
            }
        }