# Create bundle
  git bundle create $BundleName $tagName $branchName

  use HEAD tag
  <pre>
  git bundle create repo.bundle HEAD master
  </pre>

  create new tag
  <pre>
  git tag -a v1.0 -m 'my version 1.0'
  git bundle create v1.0.bundle v1.0 master
  </pre>

  create new branch with HEAD tag
  <pre>
  git branch bundleTest
  git checkout bundleTest
  git bundle create branchHEAD.bundle HEAD bundleTest
  </pre>

  create new branch with new tag
  <pre>
  git tag -a v2.0 -m 'my version 2.0'
  git bundle create branchTag.bundle v2.0 bundleTest
  </pre>
