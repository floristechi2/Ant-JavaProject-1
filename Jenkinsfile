stage 'Init'
node {
  checkout scm
  sh 'echo $BRANCH_NAME'
}
if (env.BRANCH_NAME == 'master') {
  stage 'Only on master'
  println 'This happens only on master'
  println "Current branch ${env.BRANCH_NAME}"
} else {
  stage 'Other branches'
  println "Current branch ${env.BRANCH_NAME}"
}

