  pipeline {
     agent {
         label {
              label "built-in"
              customWorkspace "/mnt/23Q2-multibranch"

               }

            }
     stages {
        
           stage ("23Q2") {
                 steps {
                   sh "sudo rm -rf *"
                   sh "sudo yum install git -y"
                    sh "sudo git clone https://github.com/pritam-jagtap/assignments-multibranch.git -b 23Q2"
                   sh "sudo yum install httpd -y"
                   sh "sudo service httpd start"
                   sh " sudo chmod -R  /mnt/23Q2-multibranch/assignments-multibranch/index.html"
                   sh "sudo mv /mnt/23Q2-multibranch/assignments-multibranch/index.html /var/www/html " 
                   sh "sudo chmod -R 777 /var/www/html/index.html"
                   sh "sudo service httpd restart"           
                       }
                        }
           

           }
          

}
