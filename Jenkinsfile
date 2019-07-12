node ("master") {
    stage ("scm")
    {
   git 'https://github.com/ghanigreen/maven_demo.git'
   //sh label: '', script: 'git clone https://github.com/ghanigreen/maven_demo.git' 
   // sh 'git clone https://github.com/ghanigreen/maven_demo.git'
    }
    stage ("build")
    {
    sh label: '', script: 'mvn clean package'
    }
    stage ("deploy")
    {
       // bat 'copy "C:\\Program Files (x86)\\Jenkins\\workspace\\pipedemo1\\gameoflife-web\\target\\gameoflife.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0_Tomcat10\\webapps"'
       
       sh 'cp -R "C:/Program Files (x86)/Jenkins/workspace/pipedemo1/gameoflife-web/target/gameoflife.war" "C:/Program Files/Apache Software Foundation/Tomcat 9.0/webapps/"'
    }

    
    
}
