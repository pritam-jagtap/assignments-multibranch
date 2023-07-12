  pipeline {
     agent {
         label {
              label "built-in"
              customWorkspace "/mnt/assignments"

               }

            }
     stages {
         stage ("23Q1") {
                 steps {
                    sh "sudo rm -rf *"
                   sh "sudo yum install git -y"
                    sh "sudo git clone https://github.com/pritam-jagtap/assignments-multibranch.git -b 23Q1"
                   sh "sudo yum install httpd -y"
                   sh "sudo service httpd start"
                   sh "sudo mv index.html /var/www/html " 
                   sh "sudo chmod -R 777 /var/www/html/index.html"
                   sh "sudo service httpd restart"           
                       }
                        }
       /*    stage ("23Q2") {
                 steps {
                   sh "sudo yum install git -y"
                    sh "sudo git clone https://github.com/pritam-jagtap/assignments-multibranch.git -b 23Q2"
                   sh "sudo yum install httpd -y"
                   sh "sudo service httpd start"
                   sh "sudo mv /mnt/assignments/index.html /var/www/html " 
                   sh "chmod -R 777 /var/www/html/index.html"
                   sh "sudo service httpd restart"           
                       }
                        }
           stage ("23Q3") {
                 steps {
                   sh "sudo yum install git -y"
                    sh "sudo git clone https://github.com/pritam-jagtap/assignments-multibranch.git -b 23Q3"
                   sh "sudo yum install httpd -y"
                   sh "sudo service httpd start"
                   sh "sudo mv /mnt/assignments/index.html /var/www/html " 
                   sh "chmod -R 777 /var/www/html/index.html"
                   sh "sudo service httpd restart"           
                       }
                        }  */

           }
          

}
