1.���нӿں���ҵ������ͬ
  debug_print: ���ڲ��Դ�ӡ��
2.˽�з���������
	a.__next_token(self)
	  ����lua table string, ��ת���� python��dict��list
	  ����ҵҪ������key�Ƿ���string��int��value�Ƿ�Ϊtable, nil, int, string, boolean
	  ���ӷ���������__parse_white(self)�������ո񣬻س��ȣ�__parse_comments(self)�� ����ע�ͣ�
			__parse_luatbl(self)�� ����table���� __parse_bracket(self)������[]�� __parse_string(self):�����ַ����� __parse_num(self)��������ֵ
	  
	b. __dump_parse(self)
       ��Աתlua table������dict
	   ���ӷ���������__dump_parse_string(self, to_parse_str)�������ַ�����__dump_parse_dict(self, to_parse_dict)�������ֵ䣻
	   ____dump_parse_list(self, to_parse_arr)������list��__dump_parse_other(self, value)������boolean��none��num������ 
	   
    c. __save_file(self, f, s), __read_file(self, f)
		��ȡ�ļ�
	
	e. __deep_copy(self, input_dict)
		�����ֵ䣬ȡ�����Ϸ�key
	  