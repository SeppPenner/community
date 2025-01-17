<!---
This is an autogenerated file!

Please do not edit this file directly, but instead make changes to the
sigs.yaml file in the project root.

To understand how this file is generated, see https://git.k8s.io/community/generator/README.md
--->
# Apps Special Interest Group

Covers deploying and operating applications in Kubernetes. We focus on the developer and devops experience of running applications in Kubernetes. We discuss how to define and run apps in Kubernetes, demo relevant tools and projects, and discuss areas of friction that can lead to suggesting improvements or feature requests.

The [charter](charter.md) defines the scope and governance of the Apps Special Interest Group.

## Meetings
* Regular SIG Meeting: [Mondays at 9:00 PT (Pacific Time)](https://docs.google.com/document/d/1FQx0BPlkkl1Bn0c9ocVBxYIKojpmrS1CFP5h0DI68AE/edit) (biweekly). [Convert to your timezone](http://www.thetimezoneconverter.com/?t=9:00&tz=PT%20%28Pacific%20Time%29).
  * [Meeting notes and Agenda](https://docs.google.com/document/d/1LZLBGW2wRDwAfdBNHJjFfk9CFoyZPcIYGWU7R1PQ3ng/edit#).
  * [Meeting recordings](https://www.youtube.com/playlist?list=PL69nYSiGNLP2LMq7vznITnpd2Fk1YIZF3).

## Leadership

### Chairs
The Chairs of the SIG run operations and processes governing the SIG.

* Janet Kuo (**[@janetkuo](https://github.com/janetkuo)**), Google
* Kenneth Owens (**[@kow3ns](https://github.com/kow3ns)**), Google
* Matt Farina (**[@mattfarina](https://github.com/mattfarina)**), Samsung SDS
* Adnan Abdulhussein (**[@prydonius](https://github.com/prydonius)**), VMware

## Contact
* [Slack](https://kubernetes.slack.com/messages/sig-apps)
* [Mailing list](https://groups.google.com/forum/#!forum/kubernetes-sig-apps)
* [Open Community Issues/PRs](https://github.com/kubernetes/community/labels/sig%2Fapps)

## Subprojects

The following subprojects are owned by sig-apps:
- **application**
  - Description: Application metadata descriptor CRD
  - Owners:
    - https://raw.githubusercontent.com/kubernetes-sigs/application/master/OWNERS
- **examples**
  - Owners:
    - https://raw.githubusercontent.com/kubernetes/examples/master/OWNERS
- **execution-hook**
  - Owners:
    - https://raw.githubusercontent.com/kubernetes-sigs/execution-hook/master/OWNERS
- **kompose**
  - Owners:
    - https://raw.githubusercontent.com/kubernetes/kompose/master/OWNERS
  - Contact
    - Slack: [#kompose](https://kubernetes.slack.com/messages/kompose)
- **workloads-api**
  - Description: The core workloads API, which is composed of the CronJob, DaemonSet, Deployment, Job, ReplicaSet, ReplicationController, and StatefulSet kinds
  - Owners:
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/apis/apps/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/apis/batch/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/apis/core/v1/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/apis/extensions/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/cronjob/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/daemon/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/deployment/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/disruption/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/history/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/job/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/replicaset/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/replication/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/controller/statefulset/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/registry/apps/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/registry/batch/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/pkg/registry/extensions/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/staging/src/k8s.io/api/apps/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/staging/src/k8s.io/api/batch/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/staging/src/k8s.io/api/core/v1/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/staging/src/k8s.io/api/extensions/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/test/e2e/apps/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/test/integration/daemonset/OWNERS
    - https://raw.githubusercontent.com/kubernetes/kubernetes/master/test/integration/deployment/OWNERS

## GitHub Teams

The below teams can be mentioned on issues and PRs in order to get attention from the right people.
Note that the links to display team membership will only work if you are a member of the org.

| Team Name | Details | Description |
| --------- |:-------:| ----------- |
| @kubernetes/sig-apps-api-reviews | [link](https://github.com/orgs/kubernetes/teams/sig-apps-api-reviews) | API Changes and Reviews |
| @kubernetes/sig-apps-bugs | [link](https://github.com/orgs/kubernetes/teams/sig-apps-bugs) | Bug Triage and Troubleshooting |
| @kubernetes/sig-apps-feature-requests | [link](https://github.com/orgs/kubernetes/teams/sig-apps-feature-requests) | Feature Requests |
| @kubernetes/sig-apps-misc | [link](https://github.com/orgs/kubernetes/teams/sig-apps-misc) | General Discussion |
| @kubernetes/sig-apps-pr-reviews | [link](https://github.com/orgs/kubernetes/teams/sig-apps-pr-reviews) | PR Reviews |
| @kubernetes/sig-apps-proposals | [link](https://github.com/orgs/kubernetes/teams/sig-apps-proposals) | Design Proposals |
| @kubernetes/sig-apps-test-failures | [link](https://github.com/orgs/kubernetes/teams/sig-apps-test-failures) | Test Failures and Triage |

<!-- BEGIN CUSTOM CONTENT -->

## Goals

* Discuss running and defining applications in Kubernetes (e.g., APIs, SDKs, Controllers, package management tools, etc.)
* Work on improvements to the Workload API
* Suggest Kubernetes features where we see friction
* Be the voice of the people running applications in Kubernetes (developers and devops)
* Help people get involved in the Kubernetes community
* Show early features/demos of tools that make running apps easier

## Non-goals

* Do not endorse one particular ecosystem tool
* Do not pick which apps to run on top of Kubernetes
* Do not recommend one way to do things (e.g., picking a template language)

## [Helm](https://helm.sh) and [Charts](https://github.com/kubernetes/charts)

Helm, Charts and its other subprojects have [moved to the CNCF](https://github.com/cncf/toc/blob/master/proposals/helm.adoc).
See Helm's [community repository](https://github.com/kubernetes-helm/community) for information about the Helm project.

<!-- END CUSTOM CONTENT -->
