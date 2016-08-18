node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'

   // Get some code from a GitHub repository
    git([url: 'https://github.com/sanyo0714/pipeline-test', branch: 'develop'])



   // Mark the code build 'stage'....
   stage 'Build'
   // Run the gcc build
   sh "gcc jenkins.c -o jenkins"

    // Mark the code run 'stage'....
   stage 'Run'
   // Run the program
   sh "./jenkins"
}