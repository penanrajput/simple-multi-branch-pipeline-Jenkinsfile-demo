pipeline {
    agent any
    parameters {
        string(name: 'name', defaultValue:'Penan' )
		string(name: 'city', defaultValue:'Jalgaon' )
		string(name: 'state', defaultValue:'Maharashtra' )
		text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')

    }
    stages {
        stage('name stage') {
            steps {
                echo '${params.name} is the parameter'
            }
        }
		stage('city stage') {
            steps {
                echo '${params.city} is the parameter'
            }
        }
		stage('state stage') {
            steps {
                echo '${params.state} is the parameter'
            }
        }
		stage('BIOGRAPHY stage') {
            steps {
                echo '${params.BIOGRAPHY} is the parameter'
            }
        }
		stage('TOGGLE stage') {
            steps {
                echo '${params.TOGGLE} is the parameter'
            }
        }
		stage('CHOICE stage') {
            steps {
                echo '${params.CHOICE} is the parameter'
            }
        }
		stage('PASSWORD stage') {
            steps {
                echo '${params.PASSWORD} is the parameter'
            }
        }
    }
}
