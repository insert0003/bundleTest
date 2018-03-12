# Create bundle
  git bundle create $BundleName $tagName $branchName

  use HEAD tag
  <pre>
  git bundle create repo.bundle HEAD master
  </pre>

  create New tag
  <pre>
  git tag -a v1.0 -m 'my version 1.0'
  git bundle create v1.0.bundle v1.0 master
  </pre>
