## CloudFormation Complex Templates Repository

<p>Welcome, a collection of high-quality, real-world use case templates designed to streamline your AWS infrastructure setup.</p>

<h2>About</h2>
<p>This repository provides a range of complex CloudFormation templates, each targeting a specific use case. Whether you're deploying a static website, setting up a serverless backend for a proof of concept (POC), or tackling other infrastructure needs, you'll find ready-to-use solutions here. Each template is thoroughly documented and organized for ease of use.</p>

<h2>Repository Structure</h2>
<ul>
    <li>Each template resides in its own folder.</li>
    <li>Every folder includes a <code>README.md</code> file that explains:
        <ul>
            <li><strong>Usage</strong>: How to deploy the template.</li>
            <li><strong>Affected Resources</strong>: AWS resources that will be created, modified, or deleted.</li>
            <li><strong>Required Modifications</strong>: Any customizations needed before deployment.</li>
        </ul>
    </li>
</ul>

<h2>Getting Started</h2>
<ol>
    <li>Clone the repository:
        <pre><code>git clone https://github.com/your-repository-name.git</code></pre>
    </li>
    <li>Navigate to the template folder that matches your use case:
        <pre><code>cd templates/static-website</code></pre>
    </li>
    <li>Review the <code>README.md</code> file in the folder for deployment instructions and prerequisites.</li>
    <li>Deploy the CloudFormation template using the AWS CLI or AWS Management Console.</li>
</ol>

<h2>How to Contribute</h2>
<p>We welcome contributions from the developer community! If you have a CloudFormation template for a specific use case, please follow these steps to contribute:</p>
<ol>
    <li><strong>Fork the repository</strong> and clone your fork locally.</li>
    <li><strong>Create a new folder</strong> for your template under the <code>templates</code> directory. Use a descriptive name for the folder (e.g., <code>serverless-backend-poc</code>).</li>
    <li>Add your CloudFormation template file (e.g., <code>template.yaml</code>) and a <code>README.md</code> file.
        <ul>
            <li>The <code>README.md</code> file should include:
                <ul>
                    <li><strong>Overview</strong>: A brief description of the use case.</li>
                    <li><strong>Usage</strong>: Deployment instructions.</li>
                    <li><strong>Resources</strong>: List of AWS resources affected by the template.</li>
                    <li><strong>Modifications</strong>: Any required changes to the template before deployment.</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>Open a pull request with a descriptive title and summary of your contribution.</li>
</ol>

<h2>Contribution Guidelines</h2>
<ul>
    <li>Ensure your templates follow best practices for AWS CloudFormation.</li>
    <li>Test your templates thoroughly before submitting.</li>
    <li>Provide clear and detailed documentation.</li>
</ul>

<h2>License</h2>
<p>This repository is licensed under the <a href="LICENSE">MIT License</a>. By contributing, you agree that your contributions will be licensed under the same license.</p>

<h2>Feedback & Support</h2>
<p>If you encounter any issues or have suggestions, feel free to open an issue or submit a pull request. We appreciate your feedback and contributions!</p>

<p>Happy templating! 🚀</p>