
---
title: "InstanceGroup"
block_external_search_index: true
---



Provides an Elastic MapReduce Cluster Instance Group configuration.
See [Amazon Elastic MapReduce Documentation](https://aws.amazon.com/documentation/emr/) for more information.

> **NOTE:** At this time, Instance Groups cannot be destroyed through the API nor
web interface. Instance Groups are destroyed when the EMR Cluster is destroyed.
this provider will resize any Instance Group to zero when destroying the resource.

{{% examples %}}
## Example Usage
{{% example %}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const task = new aws.emr.InstanceGroup("task", {
    clusterId: aws_emr_cluster_tf_test_cluster.id,
    instanceCount: 1,
    instanceType: "m5.xlarge",
});
```

{{% /example %}}
{{% /examples %}}



## Create a InstanceGroup Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/emr/#InstanceGroup">InstanceGroup</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/emr/#InstanceGroupArgs">InstanceGroupArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">InstanceGroup</span><span class="p">(resource_name, opts=None, </span>autoscaling_policy=None<span class="p">, </span>bid_price=None<span class="p">, </span>cluster_id=None<span class="p">, </span>configurations_json=None<span class="p">, </span>ebs_configs=None<span class="p">, </span>ebs_optimized=None<span class="p">, </span>instance_count=None<span class="p">, </span>instance_type=None<span class="p">, </span>name=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewInstanceGroup<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/go/aws/emr?tab=doc#InstanceGroupArgs">InstanceGroupArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/go/aws/emr?tab=doc#InstanceGroup">InstanceGroup</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Emr.InstanceGroup.html">InstanceGroup</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Emr.InstanceGroupArgs.html">InstanceGroupArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">List&lt;Instance<wbr>Group<wbr>Ebs<wbr>Config<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">[]Instance<wbr>Group<wbr>Ebs<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">Instance<wbr>Group<wbr>Ebs<wbr>Config[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>autoscaling_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bid_<wbr>price</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>configurations_<wbr>json</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs_<wbr>configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">List[Instance<wbr>Group<wbr>Ebs<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs_<wbr>optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>instance_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>instance_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## InstanceGroup Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">List&lt;Instance<wbr>Group<wbr>Ebs<wbr>Config&gt;</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Running<wbr>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">[]Instance<wbr>Group<wbr>Ebs<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Running<wbr>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">Instance<wbr>Group<wbr>Ebs<wbr>Config[]</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>running<wbr>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>autoscaling_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>bid_<wbr>price</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>configurations_<wbr>json</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ebs_<wbr>configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">List[Instance<wbr>Group<wbr>Ebs<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ebs_<wbr>optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>instance_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>instance_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>running_<wbr>instance_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing InstanceGroup Resource

Get an existing InstanceGroup resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/emr/#InstanceGroupState">InstanceGroupState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/emr/#InstanceGroup">InstanceGroup</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>autoscaling_policy=None<span class="p">, </span>bid_price=None<span class="p">, </span>cluster_id=None<span class="p">, </span>configurations_json=None<span class="p">, </span>ebs_configs=None<span class="p">, </span>ebs_optimized=None<span class="p">, </span>instance_count=None<span class="p">, </span>instance_type=None<span class="p">, </span>name=None<span class="p">, </span>running_instance_count=None<span class="p">, </span>status=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetInstanceGroup<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/go/aws/emr?tab=doc#InstanceGroupState">InstanceGroupState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/go/aws/emr?tab=doc#InstanceGroup">InstanceGroup</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Emr.InstanceGroup.html">InstanceGroup</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Emr.InstanceGroupState.html">InstanceGroupState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">List&lt;Instance<wbr>Group<wbr>Ebs<wbr>Config<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Running<wbr>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">[]Instance<wbr>Group<wbr>Ebs<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Running<wbr>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>autoscaling<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bid<wbr>Price</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>configurations<wbr>Json</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs<wbr>Configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">Instance<wbr>Group<wbr>Ebs<wbr>Config[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs<wbr>Optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>running<wbr>Instance<wbr>Count</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>autoscaling_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The autoscaling policy document. This is a JSON formatted string. See [EMR Auto Scaling](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-automatic-scaling.html)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bid_<wbr>price</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}If set, the bid price for each EC2 instance in the instance group, expressed in USD. By setting this attribute, the instance group is being declared as a Spot Instance, and will implicitly create a Spot request. Leave this blank to use On-Demand Instances.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the EMR Cluster to attach to. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>configurations_<wbr>json</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A JSON string for supplying list of configurations specific to the EMR instance group. Note that this can only be changed when using EMR release 5.21 or later.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs_<wbr>configs</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancegroupebsconfig">List[Instance<wbr>Group<wbr>Ebs<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}One or more `ebs_config` blocks as defined below. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ebs_<wbr>optimized</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether an Amazon EBS volume is EBS-optimized. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>instance_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}target number of instances for the instance group. defaults to 0.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>instance_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The EC2 instance type for all instances in the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Human friendly name given to the instance group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>running_<wbr>instance_<wbr>count</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Instance<wbr>Group<wbr>Ebs<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/aws/types/input/#InstanceGroupEbsConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/aws/types/output/#InstanceGroupEbsConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/go/aws/emr?tab=doc#InstanceGroupEbsConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/go/aws/emr?tab=doc#InstanceGroupEbsConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Iops</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The number of I/O operations per second (IOPS) that the volume supports.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The volume size, in gibibytes (GiB). This can be a number from 1 - 1024. If the volume type is EBS-optimized, the minimum value is 10.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The volume type. Valid options are 'gp2', 'io1' and 'standard'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Volumes<wbr>Per<wbr>Instance</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The number of EBS Volumes to attach per instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Iops</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The number of I/O operations per second (IOPS) that the volume supports.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The volume size, in gibibytes (GiB). This can be a number from 1 - 1024. If the volume type is EBS-optimized, the minimum value is 10.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The volume type. Valid options are 'gp2', 'io1' and 'standard'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Volumes<wbr>Per<wbr>Instance</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The number of EBS Volumes to attach per instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>iops</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The number of I/O operations per second (IOPS) that the volume supports.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The volume size, in gibibytes (GiB). This can be a number from 1 - 1024. If the volume type is EBS-optimized, the minimum value is 10.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The volume type. Valid options are 'gp2', 'io1' and 'standard'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>volumes<wbr>Per<wbr>Instance</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The number of EBS Volumes to attach per instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>iops</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of I/O operations per second (IOPS) that the volume supports.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The volume size, in gibibytes (GiB). This can be a number from 1 - 1024. If the volume type is EBS-optimized, the minimum value is 10.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The volume type. Valid options are 'gp2', 'io1' and 'standard'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>volumes<wbr>Per<wbr>Instance</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of EBS Volumes to attach per instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-aws">https://github.com/pulumi/pulumi-aws</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    <dt>Notes</dt>
	<dd>This Pulumi package is based on the [`aws` Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws).</dd>
</dl>

