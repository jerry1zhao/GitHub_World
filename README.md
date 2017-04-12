footer 保持在底部的最好方法(flexbox): http://www.tuicool.com/articles/qQbMZbu

稳定、快速、免费的前端开源项目 CDN 服务 http://www.bootcdn.cn/


CREATE TABLE posttest
(
  post_id integer NOT NULL,
  title text NOT NULL,
  content text NOT NULL,
  createdate timestamp without time zone NOT NULL,
  updatedate timestamp without time zone,
  createuser integer NOT NULL,
  postheaderimage text NOT NULL,
  updateuser integer NOT NULL,
  CONSTRAINT posttest_pkey PRIMARY KEY (post_id)
)
WITH (
  OIDS=FALSE
);
ALTER TABLE posttest
  OWNER TO postgres;
  
  
  CREATE TABLE usertest
(
  user_id integer NOT NULL,
  user_name character varying(20) NOT NULL,
  name character varying(20),
  CONSTRAINT usertest_pkey PRIMARY KEY (user_id)
)
WITH (
  OIDS=FALSE
);
ALTER TABLE usertest
  OWNER TO postgres;
