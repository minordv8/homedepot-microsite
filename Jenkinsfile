#!groovy

import com.sunrun.util.ConfigurationDetails
import sunrunAwsSamCd

sunrunAwsSamCd {
  excludedEnvironments = ['devlocal', 'training', 'relcert', 'prd']
  skipKibana = true // skip kibana mining since we don't have browser logging yet :(
  cloudfrontBuild = true
  nodeBuild = false
  family = 'marketing'
  certificationEnvironment = 'majstg'
  appTemplateFile = 'appTemplate.yaml'
  requiredSystemTests = []
  configurationDetails = [:]
  configurationDetails[ConfigurationDetails.SERVICE_OWNER] = ConfigurationDetails.ServiceOwners.DEVOPS
}
