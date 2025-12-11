// ----------------------------------------------------------
// This is a Declarative Jenkins Pipeline.
// Pipelines automate steps like cloning code, building,
// testing, and deploying applications.
// ----------------------------------------------------------

pipeline {

    // ------------------------------------------------------
    // 'agent any' means this pipeline can run on ANY Jenkins node
    // (Master/Controller or any connected agent/slave).
    // ------------------------------------------------------
    agent any

    // ------------------------------------------------------
    // All work is done inside "stages".
    // Each stage represents a phase in your CI/CD process.
    // Example: clone → build → test → deploy
    // ------------------------------------------------------
    stages {

        // ------------------------ CLONE STAGE --------------------------
        stage("clone") {

            // Steps = actual actions performed inside the stage
            steps {
                // 'echo' prints output in the Jenkins console logs
                echo "I am from clone stage"

                // In a real pipeline, this is where you clone code from Git
                // Example:
                // git url: 'https://github.com/user/repo.git'
            }
        }

        // ------------------------ BUILD STAGE --------------------------
        stage("build") {
            steps {
                echo "I am from build stage"

                // In real life, build commands run here
                // Example for Maven:
                // sh 'mvn package'
            }
        }

        // ------------------------ DEPLOY STAGE --------------------------
        stage("deploy") {
            steps {
                echo "I am from deploy stage"

                // Example real deployment commands:
                // sh 'scp target/app.jar ec2-user@server:/apps/'
                // sh 'ssh ec2-user@server "systemctl restart app"'
            }
        }
    }
}
