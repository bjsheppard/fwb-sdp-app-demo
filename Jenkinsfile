on_commit {
    continuous_integration()
}

on_pull_request to: develop, {
  continuous_integration()
  docker_deploy_to dev
}

on_merge to: master, from: develop, {
  docker_deploy_to prod
}