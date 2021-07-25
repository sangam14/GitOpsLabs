# What is GitOps ?

GitOps is a way to do Continuous Delivery, it works by using Git as a source of truth for declarative infrastructure and workloads. 
For Kubernetes this means using `git push` instead of `kubectl create/apply` or `helm install/upgrade`.


" Kubernetes anti-patterns: Let's do GitOps, not CIOps! " 


# What is Progressive Delivery?

Progressive delivery is an umbrella term for advanced deployment patterns like canaries, 
feature flags and A/B testing. Progressive delivery techniques are used to reduce the risk of introducing a new software version in production by giving app developers and SRE teams a fine-grained control over the blast radius.


This Concept Started At Weaveworks, developers are responsible for operating our Weave Cloud SaaS.  
“GitOps” is our name for how we use developer tooling to drive operations.  This post talks about GitOps,
which is 90% best practices and 10% cool new stuff that we needed to build.  
Fair warning: this is what works for us, and dear reader, you may disagree. 
[Read More](https://www.weave.works/blog/gitops-operations-by-pull-reques)


The GitOps concept originated in a blog post from the software consultancy Weaveworks in 2017 ent​itled 
‘​GitOps - Operation by Pull Request​’.1 The word itself is a portmanteau of the source-control tool (Git),
and its application to software operations (Ops). It’s an echo of DevOps, an earlier and related movement that 
sought to emphasise software operations and break down silos between different teams. 
GitOps seeks to reduce load on operational teams by leveraging key features of Git that make 
reasoning about software delivery and maintenance easier. Since its inception, GitOps has grown as 
movement alongside technologies that inspired its precepts,  as well as inspiring the development of others.
These technologies include:
