pipeline {
    agent any
    stages {
        stage('Example') {
            input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "alice,bob"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
					string(name: 'defect', defaultValue: '', description: 'Enter Defect Number')
					string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
					booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
					choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
				}
            }
            steps {
                echo "Hello, ${PERSON}, nice to meet you."
            }
			steps{
				echo "Executing for defect #${defect} executing"
			}
			steps{
				echo "Executing for defect #${PERSON} executing"
			}
			steps{
				echo "Executing for defect #${TOGGLE} executing"
			}
			steps{
				echo "Executing for defect #${CHOICE} executing"
			}
        }
    }
}