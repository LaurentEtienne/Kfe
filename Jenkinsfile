node {
    stage 'Checkout'

         def branch = env.BRANCH_NAME
         echo "current branch is ${branch}"
         checkout scm

	// git branch: 'master', credentialsId: '1', url: ''
        // git branch: '${env.GIT_BRANCH}', credentialsId: '1', url: '${env.GIT_URL}'

    stage 'Build'
        sh "npm install"
        sh "npm start"
}
