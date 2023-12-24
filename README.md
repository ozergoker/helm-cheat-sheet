# Helm Cheat Sheet

![image](https://github.com/ozergoker/helm-cheat-sheet/blob/main/helm.svg)

# What is Helm?

Helm helps you manage Kubernetes applications — Helm Charts help you define, install, and upgrade even the most complex Kubernetes application.

Charts are easy to create, version, share, and publish — so start using Helm and stop the copy-and-paste.

# Chart Management

helm create <name>                      # Creates a chart directory along with the common files and directories used in a chart.
helm package <chart-path>               # Packages a chart into a versioned chart archive file.
helm lint <chart>                       # Run tests to examine a chart and identify possible issues:
helm show all <chart>                   # Inspect a chart and list its contents:
helm show values <chart>                # Displays the contents of the values.yaml file
helm pull <chart>                       # Download/pull chart 
helm pull <chart> --untar=true          # If set to true, will untar the chart after downloading it
helm pull <chart> --verify              # Verify the package before using it
helm pull <chart> --version <number>    # Default-latest is used, specify a version constraint for the chart version to use
helm dependency list <chart>            # Display a list of a chart’s dependencies:

