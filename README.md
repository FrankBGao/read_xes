# read_xes
Use Python read XES file, to transfer XES' trace information into Python dict. This program is aiming at providing a way for Python disposal XES data.<br></br>
This file just a simple function for transfer XES' trace and event information into two python dicts. One is 'trace_attri', it is the information of trace which are gained from <trace/> tag and the tags which are not event and in <trace><trace/> tag. Other is trace_event, it is the information of evnet which are gained for <event></event> tag.  <br></br>
After you gain those two dict, you could transfer them into pandas DataFrame, or you could insert them into MonogoDB. I think that may more convenience for further usage. <br></br>
The major problem is speed, this program is much slower than ProM's import. I think it may comes from anaylze XML and loops in program. If I have time I may could find out more effienct method. Therefore, if your XES file is really big, I think this program may consumes significant time. <br></br>
At last, many thinks xmltodict(https://github.com/martinblech/xmltodict), xmltodict makes this program much easier.
