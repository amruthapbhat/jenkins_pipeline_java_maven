node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'
   
   git url: 'https://github.com/amruthapbhat/jenkins_pipeline_java_maven.git'

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
   // **       in the global configuration.           
   def mvnHome = tool 'Maven'

   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build
   bat "${mvnHome}\\bin\\mvn -B verify"
}
