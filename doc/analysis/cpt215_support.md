# CPT215 support analysis command log

## Commands executed

- `rg -n "CPT215|CPT 215|ET_215|\b215\b|CPT" src`
- `rg -n "element type|element_type|mapdl|rst|rth|descriptor|topology|element library|element descriptor|mapdl" src/ansys/dpf`
- `rg -n "CPT215|CPT 215|ET_215|CPT"`
- `rg -n "mapdl_element_type|apdl_element_type|mapdl_element_type_id" src/ansys/dpf/core`
- `rg -n "mapdl::rst" src/ansys/dpf/core/operators`
- `sed -n '850,1040p' src/ansys/dpf/core/elements.py`
- `sed -n '1,220p' src/ansys/dpf/core/operators/metadata/element_types_provider.py`
- `sed -n '1,220p' src/ansys/dpf/core/operators/metadata/property_field_provider_by_name.py`
- `sed -n '1,160p' src/ansys/dpf/core/operators/result/stress.py`
- `sed -n '1,80p' src/ansys/dpf/core/operators/build.py`
- `nl -ba src/ansys/dpf/core/elements.py | sed -n '880,1020p'`
- `nl -ba src/ansys/dpf/core/operators/metadata/property_field_provider_by_name.py | sed -n '20,180p'`
- `nl -ba src/ansys/dpf/core/operators/metadata/element_types_provider.py | sed -n '20,140p'`
- `nl -ba src/ansys/dpf/core/operators/result/stress.py | sed -n '1,220p'`
- `nl -ba src/ansys/dpf/core/operators/build.py | sed -n '1,80p'`
