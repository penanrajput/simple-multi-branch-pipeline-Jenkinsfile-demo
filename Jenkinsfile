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
        stage('test') {
            steps {
                echo '${params. name} is the parameter'
            }
        }
    }
}
