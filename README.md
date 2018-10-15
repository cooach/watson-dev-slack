# watson-dev-slack
// in the constructor, letting the SDK manage the IAM token
const discovery = new DiscoveryV1({
  url: '<service_url>',
  version: '<version-date>',
  iam_apikey: '<iam_api_key>',
  iam_url: '<iam_url>', // optional - the default value is https://iam.bluemix.net/identity/token
});
// in the constructor, assuming control of managing IAM token
const discovery = new DiscoveryV1({
  url: '<service_url>',
  version: '<version-date>',
  iam_access_token: '<access-token>'
});
  // after instantiation, assuming control of managing IAM token
const discovery = new DiscoveryV1({
  url: '<service_url>',
  version: '<version-date>'
});

discovery.setAccessToken('<access-token>')
