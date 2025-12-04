/**********************************************
 * SCRIPTED PIPELINE - POC EXAMPLE
 **********************************************/

// STEP 1: Select a Jenkins agent (any available node/agent)
node {

    /*************** Stage 1: Checkout ***************/
    stage('Checkout') {
        echo "Step 1: Fetching source code from Git..."

        // Replace this with your repo URL
        git 'https://github.com/your-username/scripted-poc.git'
    }

    /*************** Stage 2: Build ***************/
    stage('Build') {
        echo "Step 2: Building the application..."

        // Put your build commands here
        // For Maven:
        // sh 'mvn clean package'

        // For Node.js:
        // sh 'npm install'
    }

    /*************** Stage 3: Test ***************/
    stage('Test') {
        echo "Step 3: Running tests..."

        // For Maven:
        // sh 'mvn test'

        // For Node.js:
        // sh 'npm test'
    }

    /*************** Stage 4: Deploy ***************/
    stage('Deploy') {
        echo "Step 4: Simulating deployment..."

        // Just a POC, so we simulate deploy
        sh 'echo Deployment successful!'
    }

    /*************** Stage 5: Cleanup ***************/
    stage('Cleanup') {
        echo "Step 5: Cleaning workspace..."

        // Delete workspace after build
        deleteDir()
    }
}
