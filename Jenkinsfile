pipeline {
    agent any
    stages {
        stage('Testing Input Feature') {
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
            steps {
                echo "Hello, ${NAME}, nice to meet you."
				echo "Executing for defect #${DEFECT} "
				echo "Executing for toggle = ${TOGGLE} "
				echo "Executing for choice = ${CHOICE} "
            }
		}	
    }
}