pipeline
{
agent any

stages
{
stage('Build')
{
steps
{
bat "mvn clean"
}

}
stage('deploy')
{
steps{
echo 'deploying the code'
}

}
stage('test')
{
steps{
bat "mvn test"
}

}

stage('Unit Testing')
{
steps{
bat "mvn compile"
}

}
stage('Release')
{
when{
branch "origin/master"
}
steps{
echo 'releasing the project'
}

}



}

}