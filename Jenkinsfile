@NonCPS printCauses() {
  def causes = currentBuild.rawBuild.getCauses(Cause.UpstreamCause)
  if (causes) {
    println "Triggered by project ${causes.getUpstreamProject()}"
  } else {
    println "Not triggered by upstream"
  }
}

printCauses()

def pipe = new org.typo3.chefci.v1.Pipeline()
pipe.execute()
