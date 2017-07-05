# facultydashxblock

The xblock in this repository works on open edX platform.

#### Requirements
[course_dashboard_api](https://github.com/jaygoswami2303/course_dashboard_api.git)

### Installation

* Clone the repository:

  https://github.com/jaygoswami2303/facultydashxblock.git
  
* Run the command 
```bash
sudo -u edxapp/edx/bin/pip.edxapp install /path/to/your/block
```

* Add the name of the xblock (facultydashxblock) in the key ‘INSTALLED_APPS’ in python files /edx/app/edxapp/edx-platform/lms/envs/common.py and /edx/app/edxapp/edx-platform/cms/envs/common.py

```python
INSTALLED_APPS = (

...

‘facultydashxblock’ ,

)
```

* Restart LMS and CMS servers by the command:
```bash
sudo /edx/bin/supervisorctl restart edxapp:
```
