<template>
	<div class="content-section documentation">
		<TabView>
			<TabPanel header="Documentation">
				<h5>Import</h5>
<CodeHighlight lang="javascript">
import InputSwitch from 'primevue/inputswitch';
</CodeHighlight>

				<h5>Getting Started</h5>
				<p>Two-way binding to a boolean property is defined using the standard v-model directive.</p>
<CodeHighlight>
&lt;InputSwitch v-model="checked" /&gt;
</CodeHighlight>

<CodeHighlight lang="js">
export default {
	data() {
		return {
			checked: false
		}
	}
}
</CodeHighlight>

				<p>As model is two-way binding enabled, setting the bound value as true displays the state as checked by default.</p>

<CodeHighlight lang="js">
export default {
	data() {
		return {
			checked: true
		}
	}
}
</CodeHighlight>

				<h5>Properties</h5>
                <p>Any property such as name and placeholder are passed to the underlying input element. Following are the additional properties to configure the component.</p>
				<div class="doc-tablewrapper">
					<table class="doc-table">
						<thead>
                            <tr>
                                <th>Name</th>
                                <th>Type</th>
                                <th>Default</th>
                                <th>Description</th>
                            </tr>
						</thead>
						<tbody>
                            <tr>
                                <td>modelValue</td>
                                <td>boolean</td>
                                <td>null</td>
                                <td>Specifies whether a inputswitch should be checked or not.</td>
                            </tr>
						</tbody>
					</table>
				</div>

				<h5>Events</h5>
				<p>Any valid event such as focus, blur and input are passed to the underlying input element. Following are the additional events to configure the component.</p>

				<h5>Styling</h5>
				<p>Following is the list of structural style classes, for theming classes visit <router-link to="/theming">theming</router-link> page.</p>
				<div class="doc-tablewrapper">
					<table class="doc-table">
						<thead>
                            <tr>
                                <th>Name</th>
                                <th>Element</th>
                            </tr>
						</thead>
						<tbody>
                            <tr>
                                <td>p-inputswitch</td>
                                <td>Container element.</td>
                            </tr>
                            <tr>
                                <td>p-inputswitch-checked</td>
                                <td>Container element in active state.</td>
                            </tr>
                            <tr>
                                <td>p-inputswitch-slider</td>
                                <td>Slider element behind the handle.</td>
                            </tr>
						</tbody>
					</table>
				</div>

				<h5>Dependencies</h5>
				<p>None.</p>
			</TabPanel>

			<TabPanel header="Source">
				<a href="https://github.com/primefaces/primevue/tree/master/src/views/inputswitch" class="btn-viewsource" target="_blank" rel="noopener noreferrer">
					<span>View on GitHub</span>
				</a>
<CodeHighlight>
<template v-pre>
&lt;h3&gt;Basic&lt;/h3&gt;
&lt;InputSwitch v-model="checked1" /&gt;

&lt;h3&gt;Preselection&lt;/h3&gt;
&lt;InputSwitch v-model="checked2" /&gt;
</template>
</CodeHighlight>

<CodeHighlight lang="javascript">
export default {
	data() {
		return {
			checked1: false,
			checked2: true
		}
	}
}
</CodeHighlight>
			</TabPanel>
		</TabView>
	</div>
</template>