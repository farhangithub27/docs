
---
title: "Monitor"
block_external_search_index: true
---



Manages a V2 monitor resource within OpenStack.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as openstack from "@pulumi/openstack";

const monitor1 = new openstack.loadbalancer.Monitor("monitor_1", {
    delay: 20,
    maxRetries: 5,
    poolId: openstack_lb_pool_v2_pool_1.id,
    timeout: 10,
    type: "PING",
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-openstack/blob/master/website/docs/r/lb_monitor_v2.html.markdown.



## Create a Monitor Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/loadbalancer/#Monitor">Monitor</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/loadbalancer/#MonitorArgs">MonitorArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">Monitor</span><span class="p">(resource_name, opts=None, </span>admin_state_up=None<span class="p">, </span>delay=None<span class="p">, </span>expected_codes=None<span class="p">, </span>http_method=None<span class="p">, </span>max_retries=None<span class="p">, </span>max_retries_down=None<span class="p">, </span>name=None<span class="p">, </span>pool_id=None<span class="p">, </span>region=None<span class="p">, </span>tenant_id=None<span class="p">, </span>timeout=None<span class="p">, </span>type=None<span class="p">, </span>url_path=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewMonitor<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/loadbalancer?tab=doc#MonitorArgs">MonitorArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/loadbalancer?tab=doc#Monitor">Monitor</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Loadbalancer.Monitor.html">Monitor</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.LoadBalancer.MonitorArgs.html">MonitorArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>admin_<wbr>state_<wbr>up</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>expected_<wbr>codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>http_<wbr>method</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>max_<wbr>retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>retries_<wbr>down</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>pool_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tenant_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url_<wbr>path</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## Monitor Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>admin_<wbr>state_<wbr>up</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>expected_<wbr>codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>http_<wbr>method</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>max_<wbr>retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>max_<wbr>retries_<wbr>down</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>pool_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>tenant_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>url_<wbr>path</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing Monitor Resource

Get an existing Monitor resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/loadbalancer/#MonitorState">MonitorState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/loadbalancer/#Monitor">Monitor</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>admin_state_up=None<span class="p">, </span>delay=None<span class="p">, </span>expected_codes=None<span class="p">, </span>http_method=None<span class="p">, </span>max_retries=None<span class="p">, </span>max_retries_down=None<span class="p">, </span>name=None<span class="p">, </span>pool_id=None<span class="p">, </span>region=None<span class="p">, </span>tenant_id=None<span class="p">, </span>timeout=None<span class="p">, </span>type=None<span class="p">, </span>url_path=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetMonitor<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/loadbalancer?tab=doc#MonitorState">MonitorState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/loadbalancer?tab=doc#Monitor">Monitor</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Loadbalancer.Monitor.html">Monitor</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Loadbalancer.MonitorState.html">MonitorState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>admin<wbr>State<wbr>Up</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>expected<wbr>Codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>http<wbr>Method</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Retries<wbr>Down</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>pool<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tenant<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url<wbr>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>admin_<wbr>state_<wbr>up</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The administrative state of the monitor.
A valid value is true (UP) or false (DOWN).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The time, in seconds, between sending probes to members.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>expected_<wbr>codes</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. Expected HTTP codes
for a passing HTTP(S) monitor. You can either specify a single status like
"200", or a range like "200-202".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>http_<wbr>method</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. The HTTP method used
for requests by the monitor. If this attribute is not specified, it
defaults to "GET".
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>retries</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures before
changing the member's status to INACTIVE. Must be a number between 1
and 10.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>retries_<wbr>down</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of permissible ping failures befor changing the member's
status to ERROR. Must be a number between 1 and 10 (supported only in Octavia).
Changing this updates the max_retries_down of the existing monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Name of the Monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>pool_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The id of the pool that this monitor will be assigned to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region in which to obtain the V2 Networking client.
A Networking client is needed to create an . If omitted, the
`region` argument of the provider is used. Changing this creates a new
monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tenant_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for admins. The UUID of the tenant who owns
the monitor.  Only administrative users can specify a tenant UUID
other than their own. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Maximum number of seconds for a monitor to wait for a
ping reply before it times out. The value must be less than the delay
value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of probe, which is PING, TCP, HTTP, HTTPS,
TLS-HELLO or UDP-CONNECT (supported only in Octavia), that is sent by the load
balancer to verify the member state. Changing this creates a new monitor.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url_<wbr>path</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Required for HTTP(S) types. URI path that will be
accessed if monitor type is HTTP or HTTPS.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}











<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-openstack">https://github.com/pulumi/pulumi-openstack</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>

