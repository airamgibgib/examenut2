pipeline {
agent any
stages {
stage ('Checkout GIthub') {
steps {
sh "mvn clean compile test"
}
}
stage ('Compile Pro_CalculadoraACNI') {
steps {
sh "mvn -f pom.xml clean install -Dmaven.test.skip=true"
}
}
stage ('Unit Test') {
steps {
echo "Unit test"
}
}
}
}
