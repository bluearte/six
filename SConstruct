import excons
import six

env = excons.MakeBaseEnv()

prjs = [
   {
      "name": "six",
      "type": "install",
      "install": {excons.OutputBaseDirectory() + "/python": ["six.py"]}
   }
]

excons.DeclareTargets(env, prjs)

excons.EcosystemDist(env, "six.env", {"six": ""}, version=six.__version__)