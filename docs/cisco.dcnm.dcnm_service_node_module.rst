.. _cisco.dcnm.dcnm_service_node_module:


****************************
cisco.dcnm.dcnm_service_node
****************************

**Create/Modify/Delete service node based on type and attached interfaces from a DCNM managed VXLAN fabric.**


Version added: 0.9.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- Create/Modify/Delete service node based on type and attached interfaces from a DCNM managed VXLAN fabric.




Parameters
----------

.. raw:: html

    <table  border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="2">Parameter</th>
            <th>Choices/<font color="blue">Defaults</font></th>
            <th width="100%">Comments</th>
        </tr>
            <tr>
                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>config</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=dictionary</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>List of details of service nodes being managed</div>
                </td>
            </tr>
                                <tr>
                    <td class="elbow-placeholder"></td>
                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>attach_interface</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>List of switch interfaces where the service node will be attached</div>
                </td>
            </tr>
            <tr>
                    <td class="elbow-placeholder"></td>
                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>form_factor</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                        <b>Default:</b><br/><div style="color: blue">"physical"</div>
                </td>
                <td>
                        <div>Name of the form factor of the service node</div>
                </td>
            </tr>
            <tr>
                    <td class="elbow-placeholder"></td>
                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>name</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>Name of service node</div>
                </td>
            </tr>
            <tr>
                    <td class="elbow-placeholder"></td>
                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>svc_int_name</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>Name of the service interface</div>
                </td>
            </tr>
            <tr>
                    <td class="elbow-placeholder"></td>
                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>switches</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>IP address of the switch where service node will be added/deleted</div>
                </td>
            </tr>
            <tr>
                    <td class="elbow-placeholder"></td>
                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>type</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                        <b>Default:</b><br/><div style="color: blue">"firewall"</div>
                </td>
                <td>
                        <div>Name of the service node type</div>
                </td>
            </tr>

            <tr>
                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>fabric</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>Name of attached easy fabric to which service node is attached</div>
                </td>
            </tr>
            <tr>
                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>service_fabric</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                         / <span style="color: red">required</span>
                    </div>
                </td>
                <td>
                </td>
                <td>
                        <div>Name of external fabric where the service node is located</div>
                </td>
            </tr>
            <tr>
                <td colspan="2">
                    <div class="ansibleOptionAnchor" id="parameter-"></div>
                    <b>state</b>
                    <a class="ansibleOptionLink" href="#parameter-" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                    </div>
                </td>
                <td>
                        <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                    <li><div style="color: blue"><b>merged</b>&nbsp;&larr;</div></li>
                                    <li>replaced</li>
                                    <li>overridden</li>
                                    <li>deleted</li>
                                    <li>query</li>
                        </ul>
                </td>
                <td>
                        <div>The state of DCNM after module completion.</div>
                </td>
            </tr>
    </table>
    <br/>




Examples
--------

.. code-block:: yaml+jinja

    This module supports the following states:

    Merged:
      Service Nodes defined in the playbook will be merged into the service fabric.
        - If the service node does not exist it will be added.
        - If the service node exists but properties managed by the playbook are different
          they will be updated if possible.
        - Service Nodes that are not specified in the playbook will be untouched.

    Replaced:
      Service Nodes defined in the playbook will be replaced in the service fabric.
        - If the service node does not exist it will be added.
        - If the service node exists but properties managed by the playbook are different
          they will be updated if possible.
        - Properties that can be managed by the module but are not specified
          in the playbook will be deleted or defaulted if possible.
        - Service Nodes that are not specified in the playbook will be untouched.

    Overridden:
      Service Node defined in the playbook will be overridden in the service fabric.
        - If the service node does not exist it will be added.
        - If the service node exists but properties managed by the playbook are different
          they will be updated if possible.
        - Properties that can be managed by the module but are not specified
          in the playbook will be deleted or defaulted if possible.
        - Service Nodes that are not specified in the playbook will be deleted.

    Deleted:
      Service Node defined in the playbook will be deleted.
      If no Service Nodes are provided in the playbook, all service node present on that DCNM fabric will be deleted.

    Query:
      Returns the current DCNM state for the service node listed in the playbook.

    - name: Merge Service Nodes
      cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: merged
        config:
        - name: SN-11
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: Ethernet1/1
          switches:
          - 192.168.1.224
        - name: SN-12
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: vPC1
          switches:  # up to two switches, if two switches are provided, vpc is only option
          - 192.168.1.224
          - 192.168.1.225

    - name: Replace Service Nodes form factor/type parameter
      cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: replaced
        config:
        - name: SN-11
          type: firewall
       #  Replace can only modify the form factor
       #  form_factor: virtual  # the virtual will be changed to new physical
       #  form_factor: physical
          svc_int_name: svc1
          attach_interface: Ethernet1/1
          switches:
          - 192.168.1.224
       #   Nothing will be replaced in the below service node as there is no change
       #   Dont touch this if its present on DCNM
       # - name: SN-12
       #   type: firewall
       #   form_factor: virtual
       #   svc_int_name: svc1
       #   attach_interface: vPC1
       #   switches:  # up to two switches, if two switches are provided, vpc is only option
       #   - 192.168.1.224
       #   - 192.168.1.225

    - name: Override Service Nodes
      cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: overridden
        config:
       # Create this service node
         - name: SN-13
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: Ethernet1/1
          switches:
          - 192.168.1.224
       # Delete this service node from the DCNM
       # - name: SN-11
       #   type: firewall
       #   form_factor: virtual
       #   svc_int_name: svc1
       #   attach_interface: Ethernet1/1
       #   switches:
       #   - 192.168.1.224
       # Delete this service node from the DCNM
       # - name: SN-12
       #   type: firewall
       #   form_factor: virtual
       #   svc_int_name: svc1
       #   attach_interface: vPC1
       #   switches:  # up to two switches, if two switches are provided, vpc is only option
       #   - 192.168.1.224
       #   - 192.168.1.225

    - name: Delete selected Service Nodes
       cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: deleted
        config:
        - name: SN-11
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: Ethernet1/1
          switches:
          - 192.168.1.224
        - name: SN-12
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: vPC1
          switches:  # up to two switches, if two switches are provided, vpc is only option
          - 192.168.1.224
          - 192.168.1.225

    - name: Delete all the Service Nodes
      cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: deleted

    - name: Query Service Nodes state for SN-11 and SN-12
      cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: query
        config:
        - name: SN-11
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: Ethernet1/1
          switches:
          - 192.168.1.224
        - name: SN-12
          type: firewall
          form_factor: virtual
          svc_int_name: svc1
          attach_interface: vPC1
          switches:  # up to two switches, if two switches are provided, vpc is only option
          - 192.168.1.224
          - 192.168.1.225

    - name: Query all the Service Nodes
      cisco.dcnm.dcnm_service_node:
        fabric: Fabric1
        service_fabric: external
        state: query




Status
------


Authors
~~~~~~~

- Karthik Babu Harichandra Babu
