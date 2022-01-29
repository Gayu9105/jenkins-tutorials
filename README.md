# jenkins-tutorials

1. Jenkins installation


2. Github account, github plugin, github token


3. Pipeline using Pipeline script

    Dashboard > New Item > Pipeline
    Definition = Pipeline script
    Enter script
    
    Windows
    ```
    pipeline {
       agent any
        stages {
            stage('build') {
                steps {
                    bat 'python -V'
                }
            }
        }
    }
    ```

    Linux
    ```
    pipeline {
       agent any
        stages {
            stage('build') {
                steps {
                    sh 'python -V'
                }
            }
        }
    }
    ```


4. JENKINSFILE using SCM

    Dashboard > New Item > Pipeline
    Pipeline script from SCM
    Enter github repo
    Credentials
    Specify branch
    Script Path = JENKINSFILE1

    Windows
    ```
    pipeline {
       agent any
        stages {
            stage('build') {
                steps {
                    bat 'python -V'
                }
            }
        }
    }
    ```

    Linux
    ```
    pipeline {
       agent any
        stages {
            stage('build') {
                steps {
                    sh 'python -V'
                }
            }
        }
    }
    ```

5. 