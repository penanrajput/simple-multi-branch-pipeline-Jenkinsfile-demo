pipeline {
    agent any
    stages {

		input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "alice,bob"
                parameters {
                    string(name: 'NAME', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
					string(name: 'DEFECT', defaultValue: '', description: 'Enter Defect Number')
					booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
					choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
				}
		}

        stage('Name') {
            
            steps {
                echo "Hello, ${NAME}, nice to meet you."
            }
		}
		stage('defect') {
			steps{
				echo "Executing for defect #${NAME} executing"
			}
		}
		stage('TOGGLE') {
			steps{
				echo "Executing for defect #${TOGGLE} executing"
			}
		}
		stage('CHOICE') {
			steps{
				echo "Executing for defect #${CHOICE} executing"
			}
		}
    }
}