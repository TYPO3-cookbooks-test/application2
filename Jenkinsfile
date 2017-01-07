def causes = currentBuild.rawBuild.getCauses()

try {
  println causes
  println causes[0].getUpstreamProject()
  println causes[0].getUpstreamUrl()
} catch (Exception e) {
  println "Exception: ${e}"
  e.printStackTrace()
}



def pipe = new org.typo3.chefci.v1.Pipeline()
pipe.execute()
