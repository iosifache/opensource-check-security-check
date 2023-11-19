---
marp: true
theme: default
paginate: true
---

<style>
img[alt~="center"] {
  display: block;
  margin: 0 auto;
}

blockquote {
    font-size: 60%;
    margin-top: auto;
}

div.twocols {
    margin-top: 35px;
    column-count: 2;
}

div.twocols p:first-child,
div.twocols h1:first-child,
div.twocols h2:first-child,
div.twocols ul:first-child,
div.twocols ul li:first-child,
div.twocols ul li p:first-child {
    margin-top: 0 !important;
}

div.twocols p.break {
    break-before: column;
    margin-top: 0;
}
</style>

<!-- _class: lead -->

# Open source, Check, Security, Check:<br/><i>A checklist for securing open source projects</i>


---

![center](images/mutablesecurity.png)

---

![height:400px center](images/army.jpg)

---

![height:400px center](images/ust.jpg)

---

![height:400px center](images/usp.png)

---

![height:400px center](images/origo.jpg)

---

![height:500px center](images/oss_dep.png)

---

<div class="twocols">

### YES,

- Large scale use in:
  - Profitable companies
  - Critical infrastructures
- Permissive licences
- Publicly reviewable code

<p class="break"></p>

### BUT

- Unpaid maintainers
- Unmaintained, vulnerable projects
- Lack of ethical security testing 
- Low-hanging fruits for threat actors

</div>

---

![height:500px center](images/sop.jpg)

---

## ~~Notations~~ Emoji time!

☑️ for (wanna-be) one-time activities
🔁 for recurrent activities
📦 for closed source friendly activities

---

<!-- _class: lead -->

### I. Proactively find vulnerabilities

---

<!-- _class: lead -->

### 1. Create and maintain a threat model ☑️🔁📦

---

![height:300px center](images/threat_model.png)

---

<!-- _class: lead -->

### 2. Check for vulnerabilities in your dependencies ☑️🔁

---

![height:500px center](images/browserify_deps.png)

---

<!-- _class: lead -->

### 3. Run security tools and constantly validate the warnings ☑️🔁📦

---

1. Run multiple tools
2. Aggregate the results (e.g., with the [SARIF](https://sarifweb.azurewebsites.net/) format)
3. Review the results
4. Suppress the false positives
5. Create automation for development environments and CI workflows

---

<!-- _class: lead -->

### 4. Integrate your project in OSS-Fuzz ☑️🔁

---

![height:500px center](images/oss_fuzz.png)

---

<!-- _class: lead -->

### II. Secure your users

---

<!-- _class: lead -->

### 1. Design your software to be secure by default ☑️🔁📦

---

![height:500px center](images/chromium_default.png)

---

<!-- _class: lead -->

### 2. Have security recommendations for users ☑️🔁📦

---

![height:500px center](images/node_recommendations.png)

---

<!-- _class: lead -->

### 3. Create SBOMs ☑️📦

---

![height:500px center](images/sbom.png)

---

<!-- _class: lead -->

### III. Establish a security reporting process

---

<!-- _class: lead -->

### 1. Have a standardised, documented process for responding to vulnerabilities ☑️📦

---

![height:500px center](images/node_crd.png)

---

<!-- _class: lead -->

### 2. Create a security policy ☑️📦

---

![height:500px center](images/ansible_policy.png)

---

<!-- _class: lead -->

### 3. Find backup security responders ☑️📦

---

![height:500px center](images/security_backup.png)

---

<!-- _class: lead -->

### 4. Be transparent and verbose with the reported vulnerabilities 🔁📦

---

![height:300px center](images/vuln_info.png)

---

![height:300px center](images/oss_fortress.png)

---

### The OSS Fortress

- Workshop for finding software vulnerabilities using open source tools
- Vulnerable-by-default Python and C web application
- Tasks (and solutions) for linting, code querying, secret scanning, dependency scanning, fuzzing, and symbolic execution
- [`iosifache/oss_fortress` on GitHub](https://github.com/iosifache/oss_fortress)
- [`ossfortress.io` as a wiki](https://ossfortress.io/)

---

![height:300px center](images/end.jpg)

---

# `ping @iosifache`

- Website: [iosifache.me](https://iosifache.me)
- GitHub: [@iosifache](https://github.com/iosifache)
- X: [@iosifache](https://x.com/iosifache)
- LinkedIn: [@iosifache](https://www.linkedin.com/in/iosifache/)
