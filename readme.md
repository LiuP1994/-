判断非中文多语言混合评论表达情感为积极或消极，结果用 0 到 1 的数字表示。由于语言是印欧语系，且不是单一语种，按照空格分词后选择使用 one-hot 形式来表示每个词，这两步都通过 sklearn 里的TfidfVectorizer 实现，然后用 sklearn.naive_bayes 里的 MultinomialNB 进行预测。
